# histogram_plot.py

import matplotlib.pyplot as plt

def plot_age_distribution():
    # Example data: Age distribution in a population
    ages = [18, 20, 22, 22, 23, 24, 25, 25, 26, 27, 28, 28, 29, 30, 30, 30, 31, 32, 33, 35, 35, 36, 38, 40, 45, 50]

    # Create bins for age ranges
    bins = range(15, 55, 5)

    # Plot histogram
    plt.figure(figsize=(10, 6))
    plt.hist(ages, bins=bins, edgecolor='black', alpha=0.7, color='skyblue')

    # Customize chart
    plt.title('Age Distribution in a Population', fontsize=16)
    plt.xlabel('Age Range', fontsize=14)
    plt.ylabel('Frequency', fontsize=14)
    plt.xticks(bins)
    plt.grid(axis='y', linestyle='--', alpha=0.7)

    # Save and display chart
    plt.tight_layout()
    plt.savefig('age_distribution_histogram.png')  # Save the figure as an image
    plt.show()

if __name__ == "__main__":
    plot_age_distribution()
